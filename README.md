# Neluonde
def count_valleys(steps):
  """Counts the number of valleys in a sequence of steps.

  Args:
    steps: A sequence of characters representing the steps.

  Returns:
    The number of valleys.
  """

  valleys = 0
  altitude = 0
  for step in steps:
    if step == 'U':
      altitude += 1
    elif step == 'D':
      altitude -= 1
      if altitude == 0:
        valleys += 1

  return valleys
